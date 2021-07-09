---
title: Combinar várias solicitações em uma chamada HTTP usando processamento JSON em lotes
description: 'Os lotes JSON permitem otimizar seu aplicativo combinando várias solicitações em um único objeto JSON. Por exemplo, um cliente talvez queira criar um modo de exibição de dados não relacionados, como:'
author: davidmu1
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 06ac2bdae205f7525b912c7ea3bd396a2cceae74
ms.sourcegitcommit: ae83b2b372902268517fd17a8b10d6d9add422af
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/08/2021
ms.locfileid: "53334805"
---
# <a name="combine-multiple-requests-in-one-http-call-using-json-batching"></a><span data-ttu-id="feff3-104">Combinar várias solicitações em uma chamada HTTP usando processamento JSON em lotes</span><span class="sxs-lookup"><span data-stu-id="feff3-104">Combine multiple requests in one HTTP call using JSON batching</span></span>

<span data-ttu-id="feff3-p102">Os lotes JSON permitem otimizar seu aplicativo combinando várias solicitações (até 20) em um único objeto JSON. Por exemplo, um cliente talvez queira criar um modo de exibição de dados não relacionados, como:</span><span class="sxs-lookup"><span data-stu-id="feff3-p102">JSON batching allows you to optimize your application by combining multiple requests (up to 20) into a single JSON object. For example, a client might want to compose a view of unrelated data such as:</span></span>

1. <span data-ttu-id="feff3-107">Uma imagem armazenada no OneDrive</span><span class="sxs-lookup"><span data-stu-id="feff3-107">An image stored in OneDrive</span></span>
2. <span data-ttu-id="feff3-108">Uma lista de tarefas de Planejador</span><span class="sxs-lookup"><span data-stu-id="feff3-108">A list of Planner tasks</span></span>
3. <span data-ttu-id="feff3-109">O calendário de um grupo</span><span class="sxs-lookup"><span data-stu-id="feff3-109">The calendar for a group</span></span>

<span data-ttu-id="feff3-110">Combinar essas três solicitações individuais em uma única solicitação em lote pode economizar latência da rede significativa para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="feff3-110">Combining these three individual requests into a single batch request can save the application significant network latency.</span></span>

> [!VIDEO https://www.youtube-nocookie.com/embed/tzWGOp8zYh8]

## <a name="first-json-batch-request"></a><span data-ttu-id="feff3-111">Primeira solicitação JSON em lotes</span><span class="sxs-lookup"><span data-stu-id="feff3-111">First JSON batch request</span></span>

<span data-ttu-id="feff3-p103">Primeiro você cria a solicitação JSON em lote do exemplo anterior. Nesse cenário, as solicitações individuais não são interdependentes de qualquer forma e, portanto, podem ser colocadas na solicitação em lotes em qualquer ordem.</span><span class="sxs-lookup"><span data-stu-id="feff3-p103">First you construct the JSON batch request for the previous example. In this scenario, the individual requests are not interdependent in any way and therefore can be placed into the batch request in any order.</span></span>

```http
POST https://graph.microsoft.com/v1.0/$batch
Accept: application/json
Content-Type: application/json
```

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "/me/drive/root:/{file}:/content"
    },
    {
      "id": "2",
      "method": "GET",
      "url": "/me/planner/tasks"
    },
    {
      "id": "3",
      "method": "GET",
      "url": "/groups/{id}/events"
    },
    {
      "id": "4",
      "url": "/me",
      "method": "PATCH",
      "body": {
        "city" : "Redmond"
      },
      "headers": {
        "Content-Type": "application/json"
      }
    }
  ]
}
```

<span data-ttu-id="feff3-p104">As respostas para solicitações em lote podem aparecer em uma ordem diferente. A propriedade `id` pode ser usada para correlacionar solicitações e respostas individuais.</span><span class="sxs-lookup"><span data-stu-id="feff3-p104">Responses to the batched requests might appear in a different order. The `id` property can be used to correlate individual requests and responses.</span></span>

```http
200 OK
Content-Type: application/json
```

```json
{
  "responses": [
    {
      "id": "1",
      "status": 302,
      "headers": {
        "location": "https://b0mpua-by3301.files.1drv.com/y23vmagahszhxzlcvhasdhasghasodfi"
      }
    },
    {
      "id": "3",
      "status": 401,
      "body": {
        "error": {
          "code": "Forbidden",
          "message": "..."
        }
      }
    },
    {
      "id": "2",
      "status": 200,
      "body": {
        "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    },
    {
      "id": "4",
      "status": 204,
      "body": null
    }
  ]
}
```

## <a name="request-format"></a><span data-ttu-id="feff3-116">Formato da solicitação</span><span class="sxs-lookup"><span data-stu-id="feff3-116">Request format</span></span>

<span data-ttu-id="feff3-117">Solicitações de lote são sempre enviadas usando `POST` para o ponto de extremidade `/$batch`.</span><span class="sxs-lookup"><span data-stu-id="feff3-117">Batch requests are always sent using `POST` to the `/$batch` endpoint.</span></span>

<span data-ttu-id="feff3-p105">O corpo da solicitação JSON em lote consiste em um único objeto JSON com uma propriedade obrigatória: `requests`. A propriedade `requests` é uma matriz de solicitações individuais. Para cada solicitação individual, as propriedades `id`, `method` e `url` propriedades são necessárias.</span><span class="sxs-lookup"><span data-stu-id="feff3-p105">A JSON batch request body consists of a single JSON object with one required property: `requests`. The `requests` property is an array of individual requests. For each individual request, the `id`, `method`, and `url` properties are required.</span></span>

<span data-ttu-id="feff3-p106">A propriedade `id` funciona principalmente como um valor de correlação para associar solicitações a respostas individuais. Isso permite que o servidor processe solicitações em lote na ordem mais eficiente.</span><span class="sxs-lookup"><span data-stu-id="feff3-p106">The `id` property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span>

<span data-ttu-id="feff3-p107">As propriedades `method` e `url` são exatamente o que você vê no início de qualquer solicitação HTTP. O método é o método HTTP e a URL é a URL de recurso para a qual a solicitação individual normalmente seria enviada.</span><span class="sxs-lookup"><span data-stu-id="feff3-p107">The `method` and `url` properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span>

<span data-ttu-id="feff3-125">As solicitações individuais podem, como opção, também conter uma propriedade `headers` e uma propriedade`body`.</span><span class="sxs-lookup"><span data-stu-id="feff3-125">Individual requests can optionally also contain a `headers` property and a `body` property.</span></span> <span data-ttu-id="feff3-126">Essas duas propriedades geralmente são objetos JSON, conforme mostrado no exemplo anterior.</span><span class="sxs-lookup"><span data-stu-id="feff3-126">Both of these properties are typically JSON objects, as shown in the previous example.</span></span> <span data-ttu-id="feff3-127">Em alguns casos, o `body` pode ser um valor codificado como URL base64 em vez de um objeto JSON; por exemplo, quando o corpo é uma imagem.</span><span class="sxs-lookup"><span data-stu-id="feff3-127">In some cases, the `body` might be a base64 URL-encoded value rather than a JSON object - for example, when the body is an image.</span></span> <span data-ttu-id="feff3-128">Quando um `body` está incluído na solicitação, o objeto `headers` deve conter um valor para `Content-Type`.</span><span class="sxs-lookup"><span data-stu-id="feff3-128">When a `body` is included with the request, the `headers` object must contain a value for `Content-Type`.</span></span>

## <a name="response-format"></a><span data-ttu-id="feff3-129">Formato de resposta</span><span class="sxs-lookup"><span data-stu-id="feff3-129">Response format</span></span>

<span data-ttu-id="feff3-p109">O formato de resposta para solicitações de lote JSON é semelhante ao formato da solicitação. A seguir estão as principais diferenças:</span><span class="sxs-lookup"><span data-stu-id="feff3-p109">The response format for JSON batch requests is similar to the request format. The following are the key differences:</span></span>

* <span data-ttu-id="feff3-132">A propriedade no objeto JSON principal é denominada `responses` em vez de `requests`.</span><span class="sxs-lookup"><span data-stu-id="feff3-132">The property in the main JSON object is named `responses` as opposed to `requests`.</span></span>
* <span data-ttu-id="feff3-133">As respostas individuais podem aparecer em uma ordem diferente das solicitações.</span><span class="sxs-lookup"><span data-stu-id="feff3-133">Individual responses might appear in a different order than the requests.</span></span>
* <span data-ttu-id="feff3-p110">Em vez de `method` e `url`, as respostas individuais têm uma propriedade `status`. O valor de `status` é um número que representa o código de status HTTP.</span><span class="sxs-lookup"><span data-stu-id="feff3-p110">Rather than `method` and `url`, individual responses have a `status` property. The value of `status` is a number that represents the HTTP status code.</span></span>

<span data-ttu-id="feff3-p111">O código de status em uma resposta de lote geralmente é `200` ou `400`. Se a solicitação em lotes em si for mal formada, o código de status será `400`. Se a solicitação de lote for analisável, o código de status será `200`. Um código de status `200` na resposta em lote não indica que as solicitações individuais no lote são bem-sucedidas. É por isso que cada resposta individual na propriedade `responses` tem um código de status.</span><span class="sxs-lookup"><span data-stu-id="feff3-p111">The status code on a batch response is typically `200` or `400`. If the batch request itself is malformed, the status code is `400`. If the batch request is parseable, the status code is `200`. A `200` status code on the batch response does not indicate that the individual requests inside the batch succeeded. This is why each individual response in the `responses` property has a status code.</span></span>

## <a name="sequencing-requests-with-the-dependson-property"></a><span data-ttu-id="feff3-141">Solicitações de sequenciamento com a propriedade dependsOn</span><span class="sxs-lookup"><span data-stu-id="feff3-141">Sequencing requests with the dependsOn property</span></span>

<span data-ttu-id="feff3-p112">As solicitações individuais podem ser executadas em uma ordem especificada pela propriedade `dependsOn`. Essa propriedade é uma matriz de cadeias de caracteres que fazem referência a `id` de uma solicitação individual diferente. Por esse motivo, os valores de `id` precisam ser exclusivos. Por exemplo, na solicitação a seguir, o cliente está especificando que as solicitações 1 e 3 devem ser executadas primeiro, em seguida a solicitação 2 e a solicitação 4.</span><span class="sxs-lookup"><span data-stu-id="feff3-p112">Individual requests can be executed in a specified order by using the `dependsOn` property. This property is an array of strings that reference the `id` of a different individual request. For this reason, the values for `id` must be unique. For example, in the following request, the client is specifying that requests 1 and 3 should be run first, then request 2, then request 4.</span></span>

```json
{
  "requests": [
    {
      "id": "1",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "2",
      "dependsOn": [ "1" ],
      "method": "GET",
      "url": "..."
    },
    {
      "id": "3",
      "method": "GET",
      "url": "..."
    },
    {
      "id": "4",
      "dependsOn": [ "2" ],
      "method": "GET",
      "url": "..."
    }
  ]
}
```

<span data-ttu-id="feff3-146">Se uma solicitação individual falhar, qualquer solicitação que dependa dessa solicitação falhará com código de status `424` (dependência com falha).</span><span class="sxs-lookup"><span data-stu-id="feff3-146">If an individual request fails, any request that depends on that request fails with status code `424` (Failed Dependency).</span></span>

## <a name="bypassing-url-length-limitations-with-batching"></a><span data-ttu-id="feff3-147">Ignorar limitações de tamanho de URL com processamento em lotes</span><span class="sxs-lookup"><span data-stu-id="feff3-147">Bypassing URL length limitations with batching</span></span>

<span data-ttu-id="feff3-p113">Um caso de uso adicional para processamento em lotes JSON é ignorar as limitações de tamanho de URL. Em casos nos quais a cláusula de filtro é complexa, o comprimento de URL pode superar limitações incorporadas a navegadores ou a outros clientes HTTP. Você pode usar processamento em lotes JSON como solução alternativa para executar essas solicitações já que a URL longa simplesmente torna-se parte da carga da solicitação.</span><span class="sxs-lookup"><span data-stu-id="feff3-p113">An additional use case for JSON batching is to bypass URL length limitations. In cases where the filter clause is complex, the URL length might surpass limitations built into browsers or other HTTP clients. You can use JSON batching as a workaround for running these requests because the lengthy URL simply becomes part of the request payload.</span></span>

## <a name="known-issues"></a><span data-ttu-id="feff3-151">Problemas conhecidos</span><span class="sxs-lookup"><span data-stu-id="feff3-151">Known issues</span></span>

<span data-ttu-id="feff3-152">Para obter uma lista de limitações atuais relacionadas a lotes, veja [problemas conhecidos][batching-known-issues].</span><span class="sxs-lookup"><span data-stu-id="feff3-152">For a list of current limitations related to batching, see [known issues][batching-known-issues].</span></span>

[batching-known-issues]: known-issues.md#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a><span data-ttu-id="feff3-153">Confira também</span><span class="sxs-lookup"><span data-stu-id="feff3-153">See also</span></span>

<span data-ttu-id="feff3-154">Para mais informações a respeito do formato solicitação/resposta em lotes do JSON, leia [especificações da versão 4.01 do OData JSON Format](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses), seção _Solicitações e Respostas em Lote_.</span><span class="sxs-lookup"><span data-stu-id="feff3-154">For more information about the JSON batch request/response format, see the [OData JSON Format Version 4.01 specification](http://docs.oasis-open.org/odata/odata-json-format/v4.01/odata-json-format-v4.01.html#sec_BatchRequestsandResponses), section _Batch Requests and Responses_.</span></span>
