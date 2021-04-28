---
title: Listar dispositivos
description: Recupera uma lista de objetos de dispositivos registrados na organização.
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 8f17537315e97efb99837a9333cf5821818007ec
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/27/2021
ms.locfileid: "52039724"
---
# <a name="list-devices"></a><span data-ttu-id="cd300-103">Listar dispositivos</span><span class="sxs-lookup"><span data-stu-id="cd300-103">List devices</span></span>

<span data-ttu-id="cd300-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd300-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd300-105">Recupera uma lista de objetos de dispositivos registrados na organização.</span><span class="sxs-lookup"><span data-stu-id="cd300-105">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="cd300-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="cd300-106">Permissions</span></span>
<span data-ttu-id="cd300-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cd300-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cd300-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cd300-109">Permission type</span></span>      | <span data-ttu-id="cd300-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="cd300-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cd300-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cd300-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cd300-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cd300-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cd300-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cd300-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cd300-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cd300-114">Not supported.</span></span>    |
|<span data-ttu-id="cd300-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cd300-115">Application</span></span> | <span data-ttu-id="cd300-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd300-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cd300-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cd300-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="cd300-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="cd300-118">Optional query parameters</span></span>

<span data-ttu-id="cd300-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query-parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="cd300-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="cd300-120">Você pode usar `$search` nas propriedades **displayName** e **descrição**.</span><span class="sxs-lookup"><span data-stu-id="cd300-120">You can use `$search` on the **displayName** and **description** properties.</span></span> <span data-ttu-id="cd300-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="cd300-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="cd300-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="cd300-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cd300-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cd300-123">Request headers</span></span>

| <span data-ttu-id="cd300-124">Nome</span><span class="sxs-lookup"><span data-stu-id="cd300-124">Name</span></span>       |  <span data-ttu-id="cd300-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="cd300-125">Description</span></span>|
|:-----------|:------------|
| <span data-ttu-id="cd300-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="cd300-126">Authorization</span></span>  | <span data-ttu-id="cd300-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cd300-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="cd300-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="cd300-129">ConsistencyLevel</span></span> | <span data-ttu-id="cd300-130">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="cd300-130">eventual.</span></span> <span data-ttu-id="cd300-131">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="cd300-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="cd300-132">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="cd300-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cd300-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cd300-133">Request body</span></span>
<span data-ttu-id="cd300-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cd300-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd300-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd300-135">Response</span></span>

<span data-ttu-id="cd300-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="cd300-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cd300-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="cd300-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="cd300-138">Exemplo 1: Obter uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="cd300-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="cd300-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd300-139">Request</span></span>

<span data-ttu-id="cd300-140">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd300-140">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cd300-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="cd300-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="c"></a>[<span data-ttu-id="cd300-142">C#</span><span class="sxs-lookup"><span data-stu-id="cd300-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cd300-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cd300-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cd300-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cd300-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cd300-145">Java</span><span class="sxs-lookup"><span data-stu-id="cd300-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="cd300-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd300-146">Response</span></span>

<span data-ttu-id="cd300-147">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd300-147">The following is an example of the response.</span></span>

> <span data-ttu-id="cd300-148">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cd300-148">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="cd300-149">Exemplo 2: Obter apenas uma contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="cd300-149">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="cd300-150">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd300-150">Request</span></span>

<span data-ttu-id="cd300-151">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd300-151">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cd300-152">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd300-152">Response</span></span>

<span data-ttu-id="cd300-153">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd300-153">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

`294`

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="cd300-154">Exemplo 3: use $filter e $top para obter um dispositivo com um nome de exibição que comece com "a" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="cd300-154">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cd300-155">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd300-155">Request</span></span>

<span data-ttu-id="cd300-156">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd300-156">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cd300-157">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd300-157">Response</span></span>

<span data-ttu-id="cd300-158">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd300-158">The following is an example of the response.</span></span>

><span data-ttu-id="cd300-159">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cd300-159">**Note:** The response object shown here might be shortened for readability.</span></span>

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

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="cd300-160">Exemplo 4: use $search para obter dispositivos com nomes de exibição que contenham as letras "Android", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="cd300-160">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="cd300-161">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cd300-161">Request</span></span>

<span data-ttu-id="cd300-162">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="cd300-162">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_android_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="cd300-163">Resposta</span><span class="sxs-lookup"><span data-stu-id="cd300-163">Response</span></span>

<span data-ttu-id="cd300-164">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="cd300-164">The following is an example of the response.</span></span>

><span data-ttu-id="cd300-165">**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.</span><span class="sxs-lookup"><span data-stu-id="cd300-165">**Note:** The response object shown here might be shortened for readability.</span></span>

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
