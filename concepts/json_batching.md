# <a name="combine-multiple-requests-in-one-http-call-using-json-batching-preview"></a><span data-ttu-id="be591-101">Combinar várias solicitações em uma chamada HTTP usando processamento JSON em lotes (prévia)</span><span class="sxs-lookup"><span data-stu-id="be591-101">Combine multiple requests in one HTTP call using JSON batching (preview)</span></span>

<span data-ttu-id="be591-p101">Os lotes JSON permitem otimizar seu aplicativo combinando várias solicitações em um único objeto JSON. Por exemplo, um cliente talvez queira criar um modo de exibição de dados não relacionados, como:</span><span class="sxs-lookup"><span data-stu-id="be591-p101">JSON batching allows you to optimize your application by combining multiple requests into a single JSON object. For example, a client might want to compose a view of unrelated data such as:</span></span>

1. <span data-ttu-id="be591-104">Uma imagem armazenada no OneDrive</span><span class="sxs-lookup"><span data-stu-id="be591-104">An image stored in OneDrive</span></span>
2. <span data-ttu-id="be591-105">Uma lista de tarefas de Planejador</span><span class="sxs-lookup"><span data-stu-id="be591-105">A list of Planner tasks</span></span>
3. <span data-ttu-id="be591-106">O calendário de um grupo</span><span class="sxs-lookup"><span data-stu-id="be591-106">The calendar for a group</span></span>

<span data-ttu-id="be591-107">Combinar essas três solicitações individuais em uma única solicitação em lote pode economizar latência da rede significativa para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="be591-107">Combining these three individual requests into a single batch request can save the application significant network latency.</span></span>

## <a name="first-json-batch-request"></a><span data-ttu-id="be591-108">Primeira solicitação JSON em lotes</span><span class="sxs-lookup"><span data-stu-id="be591-108">First JSON batch request</span></span>

<span data-ttu-id="be591-p102">Primeiro você cria a solicitação JSON em lote do exemplo anterior. Nesse cenário, as solicitações individuais não são interdependentes de qualquer forma e, portanto, podem ser colocadas na solicitação em lotes em qualquer ordem.</span><span class="sxs-lookup"><span data-stu-id="be591-p102">First you construct the JSON batch request for the previous example. In this scenario, the individual requests are not interdependent in any way and therefore can be placed into the batch request in any order.</span></span>

```http
POST https://graph.microsoft.com/beta/$batch
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
    }
  ]
}
```

<span data-ttu-id="be591-111">As respostas para solicitações em lote podem aparecer em uma ordem diferente.</span><span class="sxs-lookup"><span data-stu-id="be591-111">Responses to the batched requests might appear in a different order. The  property can be used to correlate individual requests and responses.</span></span> <span data-ttu-id="be591-112">A propriedade `id` pode ser usada para correlacionar solicitações e respostas individuais.</span><span class="sxs-lookup"><span data-stu-id="be591-112">Responses to the batched requests might appear in a different order. The `id` property can be used to correlate individual requests and responses.</span></span>

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
        "@odata.context": "https://graph.microsoft.com/beta/$metadata#Collection(microsoft.graph.plannerTask)",
        "value": []
      }
    }
  ]
}
```

## <a name="request-format"></a><span data-ttu-id="be591-113">Formato da solicitação</span><span class="sxs-lookup"><span data-stu-id="be591-113">Request format</span></span>

<span data-ttu-id="be591-114">Solicitações de lote são sempre enviadas usando `POST` para o ponto de extremidade `/$batch`.</span><span class="sxs-lookup"><span data-stu-id="be591-114">Batch requests are always sent using `POST` to the `/$batch` endpoint.</span></span>

<span data-ttu-id="be591-115">O corpo da solicitação JSON em lote consiste em um único objeto JSON com uma propriedade obrigatória: `requests`.</span><span class="sxs-lookup"><span data-stu-id="be591-115">A JSON batch request body consists of a single JSON object with one required property: . The  property is an array of individual requests. For each individual request, the , , and  properties are required.</span></span> <span data-ttu-id="be591-116">A propriedade `requests` é uma matriz de solicitações individuais.</span><span class="sxs-lookup"><span data-stu-id="be591-116">The `requests` property is an array of individual requests.</span></span> <span data-ttu-id="be591-117">Para cada solicitação individual, as propriedades `id`, `method` e `url` são necessárias.</span><span class="sxs-lookup"><span data-stu-id="be591-117">For each individual request, the `id`, `method`, and `url` properties are required.</span></span>

<span data-ttu-id="be591-118">A propriedade `id` funciona principalmente como um valor de correlação para associar solicitações a respostas individuais.</span><span class="sxs-lookup"><span data-stu-id="be591-118">The `id` property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span> <span data-ttu-id="be591-119">Isso permite que o servidor processe solicitações em lote na ordem mais eficiente.</span><span class="sxs-lookup"><span data-stu-id="be591-119">The  property functions primarily as a correlation value to associate individual responses with requests. This allows the server to process requests in the batch in the most efficient order.</span></span>

<span data-ttu-id="be591-120">As propriedades `method` e `url` são exatamente o que você vê no início de qualquer solicitação HTTP.</span><span class="sxs-lookup"><span data-stu-id="be591-120">The `method` and `url` properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span> <span data-ttu-id="be591-121">O método é o método HTTP e a URL é a URL de recurso para a qual a solicitação individual normalmente seria enviada.</span><span class="sxs-lookup"><span data-stu-id="be591-121">The  and  properties are exactly what you would see at the start of any given HTTP request. The method is the HTTP method, and the URL is the resource URL the individual request would typically be sent to.</span></span>

<span data-ttu-id="be591-122">As solicitações individuais podem, como opção, também conter uma propriedade `headers` e uma propriedade`body`.</span><span class="sxs-lookup"><span data-stu-id="be591-122">Individual requests can optionally also contain a `headers` property and a `body` property.</span></span> <span data-ttu-id="be591-123">Essas duas propriedades geralmente são objetos JSON.</span><span class="sxs-lookup"><span data-stu-id="be591-123">Both of these properties are typically JSON objects.</span></span> <span data-ttu-id="be591-124">Em alguns casos, o `body` pode ser um valor codificado como URL base64 em vez de um objeto JSON; por exemplo, quando o corpo é uma imagem.</span><span class="sxs-lookup"><span data-stu-id="be591-124">In some cases, the `body` might be a base64 URL-encoded value rather than a JSON object - for example, when the body is an image.</span></span> <span data-ttu-id="be591-125">Quando um `body` está incluído na solicitação, o objeto `headers` deve conter um valor para `content-type`.</span><span class="sxs-lookup"><span data-stu-id="be591-125">When a `body` is included with the request, the `headers` object must contain a value for `content-type`.</span></span>

## <a name="response-format"></a><span data-ttu-id="be591-126">Formato de resposta</span><span class="sxs-lookup"><span data-stu-id="be591-126">Response format</span></span>

<span data-ttu-id="be591-p108">O formato de resposta para solicitações de lote JSON é semelhante ao formato da solicitação. A seguir estão as principais diferenças:</span><span class="sxs-lookup"><span data-stu-id="be591-p108">The response format for JSON batch requests is similar to the request format. The following are the key differences:</span></span>

* <span data-ttu-id="be591-129">A propriedade no objeto JSON principal é denominada `responses` em vez de `requests`.</span><span class="sxs-lookup"><span data-stu-id="be591-129">The property in the main JSON object is named `responses` as opposed to `requests`.</span></span>
* <span data-ttu-id="be591-130">As respostas individuais podem aparecer em uma ordem diferente das solicitações.</span><span class="sxs-lookup"><span data-stu-id="be591-130">Individual responses might appear in a different order than the requests.</span></span>
* <span data-ttu-id="be591-131">Em vez de `method` e `url`, as respostas individuais têm uma propriedade `status`.</span><span class="sxs-lookup"><span data-stu-id="be591-131">Rather than `method` and `url`, individual responses have a `status` property.</span></span> <span data-ttu-id="be591-132">O valor de `status` é um número que representa o código de status HTTP.</span><span class="sxs-lookup"><span data-stu-id="be591-132">Rather than  and , individual responses have a  property. The value of `status` is a number that represents the HTTP status code.</span></span>

<span data-ttu-id="be591-133">O código de status em uma resposta de lote geralmente é `200` ou `400`.</span><span class="sxs-lookup"><span data-stu-id="be591-133">The status code on a batch response is typically `200` or `400`.</span></span> <span data-ttu-id="be591-134">Se a solicitação de lote em si for mal formada, o código de status será `400`.</span><span class="sxs-lookup"><span data-stu-id="be591-134">If the batch request itself is malformed, the status code is `400`.</span></span> <span data-ttu-id="be591-135">Se a solicitação de lote for analisável, o código de status será `200`.</span><span class="sxs-lookup"><span data-stu-id="be591-135">If the batch request is parseable, the status code is `200`.</span></span> <span data-ttu-id="be591-136">Um código de status `200` na resposta de lote não indica que as solicitações individuais no lote foram bem-sucedidas.</span><span class="sxs-lookup"><span data-stu-id="be591-136">A `200` status code on the batch response does not indicate that the individual requests inside the batch succeeded.</span></span> <span data-ttu-id="be591-137">Por esse motivo, cada resposta individual na propriedade `responses` tem um código de status.</span><span class="sxs-lookup"><span data-stu-id="be591-137">This is why each individual response in the `responses` property has a status code.</span></span>

<span data-ttu-id="be591-138">Além da propriedade `responses`, pode haver uma propriedade `nextLink` na resposta em lotes.</span><span class="sxs-lookup"><span data-stu-id="be591-138">In addition to the `responses` property, there might be a `nextLink` property in the batch response.</span></span> <span data-ttu-id="be591-139">Isso permite que o Microsoft Graph retorne uma resposta em lotes assim que qualquer uma das solicitações individuais for concluída.</span><span class="sxs-lookup"><span data-stu-id="be591-139">This allows Microsoft Graph to return a batch response as soon as any of the individual requests has completed.</span></span> <span data-ttu-id="be591-140">Para garantir que todas as respostas individuais foram recebidas, continue a acompanhar o `nextLink` enquanto existir.</span><span class="sxs-lookup"><span data-stu-id="be591-140">To ensure that all individual responses have been received, continue to follow the `nextLink` as long as it exists.</span></span>

## <a name="sequencing-requests-with-the-dependson-property"></a><span data-ttu-id="be591-141">Solicitações de sequenciamento com a propriedade dependsOn</span><span class="sxs-lookup"><span data-stu-id="be591-141">Sequencing requests with the dependsOn property</span></span>

<span data-ttu-id="be591-142">As solicitações individuais podem ser executadas em uma ordem especificada pela propriedade `dependsOn`.</span><span class="sxs-lookup"><span data-stu-id="be591-142">Individual requests can be executed in a specified order by using the `dependsOn` property.</span></span> <span data-ttu-id="be591-143">Essa propriedade é uma matriz de cadeias de caracteres que fazem referência a `id` de uma solicitação individual diferente.</span><span class="sxs-lookup"><span data-stu-id="be591-143">This property is an array of strings that reference the `id` of a different individual request.</span></span> <span data-ttu-id="be591-144">Por esse motivo, os valores de `id` devem ser exclusivos.</span><span class="sxs-lookup"><span data-stu-id="be591-144">For this reason, the values for `id` must be unique.</span></span> <span data-ttu-id="be591-145">Por exemplo, na solicitação a seguir, o cliente está especificando que as solicitações 1 e 3 devem ser executadas primeiro, em seguida a solicitação 2 e depois a solicitação 4.</span><span class="sxs-lookup"><span data-stu-id="be591-145">For example, in the following request, the client is specifying that requests 1 and 3 should be run first, then request 2, then request 4.</span></span>

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

<span data-ttu-id="be591-146">Se uma solicitação individual falhar, qualquer solicitação que dependa dessa solicitação falhará com código de status `424` (dependência com falha).</span><span class="sxs-lookup"><span data-stu-id="be591-146">If an individual request fails, any request that depends on that request fails with status code `424` (Failed Dependency).</span></span>

## <a name="bypassing-url-length-limitations-with-batching"></a><span data-ttu-id="be591-147">Ignorar limitações de tamanho de URL com processamento em lotes</span><span class="sxs-lookup"><span data-stu-id="be591-147">Bypassing URL length limitations with batching</span></span>

<span data-ttu-id="be591-p113">Um caso de uso adicional para processamento em lotes JSON é ignorar as limitações de tamanho de URL. Em casos nos quais a cláusula de filtro é complexa, o comprimento de URL pode superar limitações incorporadas a navegadores ou a outros clientes HTTP. Você pode usar processamento em lotes JSON como solução alternativa para executar essas solicitações já que a URL longa simplesmente torna-se parte da carga da solicitação.</span><span class="sxs-lookup"><span data-stu-id="be591-p113">An additional use case for JSON batching is to bypass URL length limitations. In cases where the filter clause is complex, the URL length might surpass limitations built into browsers or other HTTP clients. You can use JSON batching as a workaround for running these requests because the lengthy URL simply becomes part of the request payload.</span></span>

## <a name="known-issues"></a><span data-ttu-id="be591-151">Problemas conhecidos</span><span class="sxs-lookup"><span data-stu-id="be591-151">Known issues</span></span>

<span data-ttu-id="be591-152">Para obter uma lista de limitações atuais relacionadas a lotes, veja [problemas conhecidos][batching-known-issues].</span><span class="sxs-lookup"><span data-stu-id="be591-152">For a list of current limitations related to batching, see [known issues][batching-known-issues].</span></span>

[batching-known-issues]: https://developer.microsoft.com/en-us/graph/docs/concepts/known_issues#json-batching
[odata-4.01-json]: https://www.oasis-open.org/committees/download.php/60365/odata-json-format-v4.01-wd02-2017-03-24.docx


## <a name="see-also"></a><span data-ttu-id="be591-153">Veja também</span><span class="sxs-lookup"><span data-stu-id="be591-153">See also</span></span>

<span data-ttu-id="be591-154">Para saber mais sobre o formato de solicitação/resposta em lote JSON, veja o [Especificação de formato OData JSON versão 4.01][odata-4.01-json], seção 18.</span><span class="sxs-lookup"><span data-stu-id="be591-154">For more information about the JSON batch request/response format, see the [OData JSON Format Version 4.01 specification][odata-4.01-json], section 18. Note that this specification is currently in a draft version, but is not expected to change.</span></span> <span data-ttu-id="be591-155">Observe que essa especificação está atualmente em uma versão de rascunho, mas alterações não são esperadas.</span><span class="sxs-lookup"><span data-stu-id="be591-155">For more information about the JSON batch request/response format, see the OData JSON Format Version 4.01 specification, section 18. Note that this specification is currently in a draft version, but is not expected to change.</span></span>

