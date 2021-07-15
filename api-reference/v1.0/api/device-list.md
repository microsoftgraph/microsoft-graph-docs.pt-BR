---
title: Listar dispositivos
description: Recupera uma lista de objetos de dispositivos registrados na organização.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: f6bddb248b42561ad253696e27c4fedce0ee243a
ms.sourcegitcommit: 6d247f44a6ee4d8515c3863ee8a2683163c9f829
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/14/2021
ms.locfileid: "53430242"
---
# <a name="list-devices"></a><span data-ttu-id="6db73-103">Listar dispositivos</span><span class="sxs-lookup"><span data-stu-id="6db73-103">List devices</span></span>

<span data-ttu-id="6db73-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6db73-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="6db73-105">Recupera uma lista de objetos de dispositivos registrados na organização.</span><span class="sxs-lookup"><span data-stu-id="6db73-105">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="6db73-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="6db73-106">Permissions</span></span>
<span data-ttu-id="6db73-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6db73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="6db73-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6db73-109">Permission type</span></span>      | <span data-ttu-id="6db73-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="6db73-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6db73-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6db73-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6db73-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6db73-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6db73-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6db73-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6db73-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6db73-114">Not supported.</span></span>    |
|<span data-ttu-id="6db73-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6db73-115">Application</span></span> | <span data-ttu-id="6db73-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6db73-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6db73-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6db73-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6db73-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="6db73-118">Optional query parameters</span></span>

<span data-ttu-id="6db73-119">Este método suporta aos parâmetros de consulta `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, e `$top` [OData](/graph/query-parameters) para ajudar a personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="6db73-119">This method supports the `$count`, `$expand`, `$filter`, `$orderBy`, `$search`, `$select`, and `$top` [OData query parameters](/graph/query-parameters) to help customize the response.</span></span> <span data-ttu-id="6db73-120">Algumas consultas são suportadas somente quando se usa o cabeçalho **ConsistencyLevel** definido como `eventual` e `$count`.</span><span class="sxs-lookup"><span data-stu-id="6db73-120">Some queries are supported only when you use the **ConsistencyLevel** header set to `eventual` and `$count`.</span></span> <span data-ttu-id="6db73-121">Para obter mais informações, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="6db73-121">For more information, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

## <a name="request-headers"></a><span data-ttu-id="6db73-122">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6db73-122">Request headers</span></span>

| <span data-ttu-id="6db73-123">Nome</span><span class="sxs-lookup"><span data-stu-id="6db73-123">Name</span></span>       |  <span data-ttu-id="6db73-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="6db73-124">Description</span></span>|
|:-----------|:------------|
| <span data-ttu-id="6db73-125">Autorização</span><span class="sxs-lookup"><span data-stu-id="6db73-125">Authorization</span></span>  | <span data-ttu-id="6db73-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6db73-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="6db73-128">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="6db73-128">ConsistencyLevel</span></span> | <span data-ttu-id="6db73-129">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="6db73-129">eventual.</span></span> <span data-ttu-id="6db73-130">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou em uso específico de `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6db73-130">This header and `$count` are required when using `$search`, or in specific usage of `$filter`.</span></span> <span data-ttu-id="6db73-131">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="6db73-131">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span> |

## <a name="request-body"></a><span data-ttu-id="6db73-132">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6db73-132">Request body</span></span>
<span data-ttu-id="6db73-133">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6db73-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6db73-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db73-134">Response</span></span>

<span data-ttu-id="6db73-135">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6db73-135">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6db73-136">Exemplos</span><span class="sxs-lookup"><span data-stu-id="6db73-136">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="6db73-137">Exemplo 1: Obter uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="6db73-137">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="6db73-138">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db73-138">Request</span></span>

<span data-ttu-id="6db73-139">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db73-139">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6db73-140">HTTP</span><span class="sxs-lookup"><span data-stu-id="6db73-140">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[<span data-ttu-id="6db73-141">C#</span><span class="sxs-lookup"><span data-stu-id="6db73-141">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="6db73-142">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6db73-142">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6db73-143">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6db73-143">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6db73-144">Java</span><span class="sxs-lookup"><span data-stu-id="6db73-144">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="6db73-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db73-145">Response</span></span>

<span data-ttu-id="6db73-146">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6db73-146">The following is an example of the response.</span></span>

> <span data-ttu-id="6db73-147">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6db73-147">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="6db73-148">Exemplo 2: Obter apenas uma contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="6db73-148">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="6db73-149">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db73-149">Request</span></span>

<span data-ttu-id="6db73-150">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db73-150">The following is an example of the request.</span></span> <span data-ttu-id="6db73-151">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` porque `$count` está na solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db73-151">This request requires the **ConsistencyLevel** header set to `eventual` because `$count` is in the request.</span></span> <span data-ttu-id="6db73-152">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="6db73-152">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6db73-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db73-153">Response</span></span>

<span data-ttu-id="6db73-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6db73-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain

294
```


### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="6db73-155">Exemplo 3: use $filter e $top para obter um dispositivo com um nome de exibição que comece com "a" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="6db73-155">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6db73-156">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db73-156">Request</span></span>

<span data-ttu-id="6db73-157">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db73-157">The following is an example of the request.</span></span> <span data-ttu-id="6db73-158">Esta solicitação exige o cabeçalho **ConsistencyLevel** definido como `eventual` e a cadeia de caracteres de consulta `$count=true` porque a solicitação tem os parâmetros de consulta `$orderBy` e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="6db73-158">This request requires the **ConsistencyLevel** header set to `eventual` and the `$count=true` query string because the request has both the `$orderBy` and `$filter` query parameters.</span></span> <span data-ttu-id="6db73-159">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="6db73-159">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6db73-160">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db73-160">Response</span></span>

<span data-ttu-id="6db73-161">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6db73-161">The following is an example of the response.</span></span>

><span data-ttu-id="6db73-162">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6db73-162">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="6db73-163">Exemplo 4: use $search para obter dispositivos com nomes de exibição que contenham as letras "Android", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="6db73-163">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="6db73-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6db73-164">Request</span></span>

<span data-ttu-id="6db73-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db73-165">The following is an example of the request.</span></span> <span data-ttu-id="6db73-166">Essa solicitação requer o header **ConsistencyLevel** definido como porque e a cadeia de caracteres de consulta `eventual` está na `$search` `$count=true` solicitação.</span><span class="sxs-lookup"><span data-stu-id="6db73-166">This request requires the **ConsistencyLevel** header set to `eventual` because `$search` and the `$count=true` query string is in the request.</span></span> <span data-ttu-id="6db73-167">Para obter mais informações sobre o uso de **ConsistencyLevel** e `$count`, consulte [Funcionalidades avançadas de consulta nos objetos de diretório do Microsoft Azure AD](/graph/aad-advanced-queries).</span><span class="sxs-lookup"><span data-stu-id="6db73-167">For more information about the use of **ConsistencyLevel** and `$count`, see [Advanced query capabilities on Azure AD directory objects](/graph/aad-advanced-queries).</span></span>

<!-- {
  "blockType": "request",
  "name": "get_android_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="6db73-168">Resposta</span><span class="sxs-lookup"><span data-stu-id="6db73-168">Response</span></span>

<span data-ttu-id="6db73-169">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="6db73-169">The following is an example of the response.</span></span>

><span data-ttu-id="6db73-170">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="6db73-170">**Note:** The response object shown here might be shortened for readability.</span></span>

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
