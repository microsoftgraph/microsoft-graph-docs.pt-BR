---
author: JeremyKelley
title: Listar pacotes
description: Listar os pacotes na unidade de um usuário
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 746cfcc09792baf5d4b6cbb19be22f3918e06d54
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047781"
---
# <a name="list-bundles"></a><span data-ttu-id="5fc68-103">Listar pacotes</span><span class="sxs-lookup"><span data-stu-id="5fc68-103">List bundles</span></span>

<span data-ttu-id="5fc68-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5fc68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5fc68-105">Obter uma lista de todos os [pacotes de][pacotes] na unidade de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5fc68-105">Get a list of all the [bundles][bundle] in a user's drive.</span></span>

## <a name="permissions"></a><span data-ttu-id="5fc68-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="5fc68-106">Permissions</span></span>

<span data-ttu-id="5fc68-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="5fc68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5fc68-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5fc68-109">Permission type</span></span>      | <span data-ttu-id="5fc68-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="5fc68-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="5fc68-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5fc68-111">Delegated (work or school account)</span></span> | <span data-ttu-id="5fc68-112">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fc68-112">Not supported.</span></span>                             |
|<span data-ttu-id="5fc68-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5fc68-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5fc68-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5fc68-114">Files.Read, Files.ReadWrite, Files.Read.All, Files.ReadWrite.All</span></span>    |
|<span data-ttu-id="5fc68-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5fc68-115">Application</span></span>          | <span data-ttu-id="5fc68-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5fc68-116">Not supported.</span></span>                                           |

## <a name="http-request"></a><span data-ttu-id="5fc68-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5fc68-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /drive/bundles
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5fc68-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="5fc68-118">Optional query parameters</span></span>

<span data-ttu-id="5fc68-119">Esse método dá suporte a [Parâmetros de consulta OData][] para filtrar e dar forma à resposta.</span><span class="sxs-lookup"><span data-stu-id="5fc68-119">This method supports the [OData Query Parameters][] to filter and shape the response.</span></span>

<span data-ttu-id="5fc68-120">Não é possível usar o `expand=children` parâmetro de consulta ao enumerar pacotes.</span><span class="sxs-lookup"><span data-stu-id="5fc68-120">You can't use the `expand=children` query parameter when enumerating bundles.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5fc68-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5fc68-121">Request headers</span></span>

| <span data-ttu-id="5fc68-122">Nome</span><span class="sxs-lookup"><span data-stu-id="5fc68-122">Name</span></span>          | <span data-ttu-id="5fc68-123">Descrição</span><span class="sxs-lookup"><span data-stu-id="5fc68-123">Description</span></span>  |
|:------------- |:------------ |
| <span data-ttu-id="5fc68-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="5fc68-124">Authorization</span></span> | <span data-ttu-id="5fc68-p102">\{token\} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5fc68-p102">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5fc68-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5fc68-127">Request body</span></span>

<span data-ttu-id="5fc68-128">Não forneça um corpo de solicitação com esse método.</span><span class="sxs-lookup"><span data-stu-id="5fc68-128">Do not supply a request body with this method.</span></span>

## <a name="response"></a><span data-ttu-id="5fc68-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fc68-129">Response</span></span>

<span data-ttu-id="5fc68-130">Se tiver êxito, essa solicitação retornará a lista de itens de pacote definidos para a unidade.</span><span class="sxs-lookup"><span data-stu-id="5fc68-130">If successful, this request returns the list of bundle items defined for the drive.</span></span>

<span data-ttu-id="5fc68-131">Leia o tópico [Respostas de erro][error-response] para obter mais informações sobre como os erros são retornados.</span><span class="sxs-lookup"><span data-stu-id="5fc68-131">Read the [Error Responses][error-response] topic for more info about how errors are returned.</span></span>

## <a name="examples"></a><span data-ttu-id="5fc68-132">Exemplos</span><span class="sxs-lookup"><span data-stu-id="5fc68-132">Examples</span></span>

### <a name="example-1-list-all-bundles-in-a-drive"></a><span data-ttu-id="5fc68-133">Exemplo 1: Listar todos os pacotes em uma unidade</span><span class="sxs-lookup"><span data-stu-id="5fc68-133">Example 1: List all bundles in a drive</span></span>

<span data-ttu-id="5fc68-134">Para solicitar uma enumeração de todos os pacotes definidos na unidade, você pode fazer uma solicitação à coleção **bundles** sem parâmetros.</span><span class="sxs-lookup"><span data-stu-id="5fc68-134">To request an enumeration of all bundles defined in the drive, you can make a request to the **bundles** collection without any parameters.</span></span>

#### <a name="request"></a><span data-ttu-id="5fc68-135">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fc68-135">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5fc68-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fc68-136">HTTP</span></span>](#tab/http)
<!-- { "blockType": "request", "name": "list-all-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles
```
# <a name="c"></a>[<span data-ttu-id="5fc68-137">C#</span><span class="sxs-lookup"><span data-stu-id="5fc68-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-all-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fc68-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fc68-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-all-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fc68-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fc68-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-all-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5fc68-140">Java</span><span class="sxs-lookup"><span data-stu-id="5fc68-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-all-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5fc68-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fc68-141">Response</span></span>

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

<span data-ttu-id="5fc68-142">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="5fc68-142">The response object shown here might be shortened for readability.</span></span>


### <a name="example-2-list-all-photo-albums-in-a-drive"></a><span data-ttu-id="5fc68-143">Exemplo 2: Listar todos os álbuns de fotos em uma unidade</span><span class="sxs-lookup"><span data-stu-id="5fc68-143">Example 2: List all photo albums in a drive</span></span>

<span data-ttu-id="5fc68-144">Para filtrar a lista de pacotes retornados de uma solicitação para a coleção bundles, você pode usar o parâmetro de cadeia de caracteres de consulta para especificar o tipo de pacote a ser retornado verificando a existência de uma faceta no `filter` pacote:</span><span class="sxs-lookup"><span data-stu-id="5fc68-144">To filter the list of bundles returned from a request to the bundles collection, you can use the `filter` query string parameter to specify the type of bundle to return by checking for the existence of a facet on the bundle:</span></span>

#### <a name="request"></a><span data-ttu-id="5fc68-145">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5fc68-145">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="5fc68-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5fc68-146">HTTP</span></span>](#tab/http)
<!-- {"blockType": "request", "name": "list-album-bundles", "tags": "service.onedrive" } -->

```msgraph-interactive
GET https://graph.microsoft.com/beta/drive/bundles?filter=bundle/album%20ne%20null
```
# <a name="c"></a>[<span data-ttu-id="5fc68-147">C#</span><span class="sxs-lookup"><span data-stu-id="5fc68-147">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-album-bundles-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5fc68-148">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5fc68-148">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-album-bundles-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5fc68-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5fc68-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-album-bundles-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5fc68-150">Java</span><span class="sxs-lookup"><span data-stu-id="5fc68-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-album-bundles-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="5fc68-151">Resposta</span><span class="sxs-lookup"><span data-stu-id="5fc68-151">Response</span></span>

<span data-ttu-id="5fc68-152">A resposta a um GET para o ponto de extremidade de pacotes é uma matriz de [recursos driveItem][] com o [pacote][].</span><span class="sxs-lookup"><span data-stu-id="5fc68-152">The response to a GET to the bundles endpoint is an array of [driveItem][] resources with the [bundle][].</span></span>
<span data-ttu-id="5fc68-153">Como todos os pacotes são itens, você pode usar todas as operações de item padrão neles.</span><span class="sxs-lookup"><span data-stu-id="5fc68-153">Because all bundles are items, you can use use all the standard item operations on them.</span></span>

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

<span data-ttu-id="5fc68-154">O objeto de resposta mostrado aqui pode ser reduzido para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="5fc68-154">The response object shown here might be shortened for readability.</span></span>


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
  "tocPath&quot;: &quot;Bundles/List"
} -->


