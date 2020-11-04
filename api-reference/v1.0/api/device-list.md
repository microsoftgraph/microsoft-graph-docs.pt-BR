---
title: Listar dispositivos
description: Recupera uma lista de objetos de dispositivos registrados na organização.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: aee70ce8dd2e308ccbd215882a11223a21a0af4f
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/04/2020
ms.locfileid: "48905250"
---
# <a name="list-devices"></a><span data-ttu-id="f671c-103">Listar dispositivos</span><span class="sxs-lookup"><span data-stu-id="f671c-103">List devices</span></span>

<span data-ttu-id="f671c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f671c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f671c-105">Recupera uma lista de objetos de dispositivos registrados na organização.</span><span class="sxs-lookup"><span data-stu-id="f671c-105">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="f671c-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="f671c-106">Permissions</span></span>
<span data-ttu-id="f671c-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f671c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="f671c-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f671c-109">Permission type</span></span>      | <span data-ttu-id="f671c-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="f671c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="f671c-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f671c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="f671c-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="f671c-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="f671c-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f671c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="f671c-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f671c-114">Not supported.</span></span>    |
|<span data-ttu-id="f671c-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f671c-115">Application</span></span> | <span data-ttu-id="f671c-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f671c-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="f671c-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f671c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="f671c-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="f671c-118">Optional query parameters</span></span>

<span data-ttu-id="f671c-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="f671c-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="f671c-120">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="f671c-120">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="f671c-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="f671c-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="f671c-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="f671c-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f671c-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f671c-123">Request headers</span></span>

| <span data-ttu-id="f671c-124">Nome</span><span class="sxs-lookup"><span data-stu-id="f671c-124">Name</span></span>       |  <span data-ttu-id="f671c-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f671c-125">Description</span></span>|
|:-----------|:------------|
| <span data-ttu-id="f671c-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="f671c-126">Authorization</span></span>  | <span data-ttu-id="f671c-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f671c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="f671c-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="f671c-129">ConsistencyLevel</span></span> | <span data-ttu-id="f671c-130">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="f671c-130">eventual.</span></span> <span data-ttu-id="f671c-131">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="f671c-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="f671c-132">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="f671c-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="f671c-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f671c-133">Request body</span></span>
<span data-ttu-id="f671c-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="f671c-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f671c-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="f671c-135">Response</span></span>

<span data-ttu-id="f671c-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f671c-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f671c-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="f671c-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="f671c-138">Exemplo 1: obter uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="f671c-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="f671c-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f671c-139">Request</span></span>

<span data-ttu-id="f671c-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f671c-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="f671c-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="f671c-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[<span data-ttu-id="f671c-142">C#</span><span class="sxs-lookup"><span data-stu-id="f671c-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f671c-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f671c-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f671c-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f671c-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f671c-145">Java</span><span class="sxs-lookup"><span data-stu-id="f671c-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="f671c-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="f671c-146">Response</span></span>

<span data-ttu-id="f671c-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f671c-147">The following is an example of the response.</span></span>

> <span data-ttu-id="f671c-p105">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f671c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="f671c-150">Exemplo 2: obter apenas uma contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="f671c-150">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="f671c-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f671c-151">Request</span></span>

<span data-ttu-id="f671c-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f671c-152">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f671c-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="f671c-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="f671c-154">C#</span><span class="sxs-lookup"><span data-stu-id="f671c-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f671c-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f671c-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f671c-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f671c-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f671c-157">Java</span><span class="sxs-lookup"><span data-stu-id="f671c-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f671c-158">Resposta</span><span class="sxs-lookup"><span data-stu-id="f671c-158">Response</span></span>

<span data-ttu-id="f671c-159">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f671c-159">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="f671c-160">Exemplo 3: use $filter e $top para obter um dispositivo com um nome de exibição que comece com ' a ', incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="f671c-160">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f671c-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f671c-161">Request</span></span>

<span data-ttu-id="f671c-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f671c-162">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f671c-163">HTTP</span><span class="sxs-lookup"><span data-stu-id="f671c-163">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="f671c-164">C#</span><span class="sxs-lookup"><span data-stu-id="f671c-164">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f671c-165">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f671c-165">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f671c-166">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f671c-166">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f671c-167">Java</span><span class="sxs-lookup"><span data-stu-id="f671c-167">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f671c-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="f671c-168">Response</span></span>

<span data-ttu-id="f671c-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f671c-169">The following is an example of the response.</span></span>

><span data-ttu-id="f671c-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f671c-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#devices",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="f671c-172">Exemplo 4: Use $search para obter dispositivos com nomes de exibição que contenham as letras "Android", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="f671c-172">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="f671c-173">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f671c-173">Request</span></span>

<span data-ttu-id="f671c-174">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="f671c-174">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="f671c-175">HTTP</span><span class="sxs-lookup"><span data-stu-id="f671c-175">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_android_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="f671c-176">C#</span><span class="sxs-lookup"><span data-stu-id="f671c-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-android-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f671c-177">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f671c-177">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-android-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f671c-178">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f671c-178">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-android-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f671c-179">Java</span><span class="sxs-lookup"><span data-stu-id="f671c-179">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-android-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="f671c-180">Resposta</span><span class="sxs-lookup"><span data-stu-id="f671c-180">Response</span></span>

<span data-ttu-id="f671c-181">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="f671c-181">The following is an example of the response.</span></span>

><span data-ttu-id="f671c-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f671c-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#devices",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0"
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- 
{
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
