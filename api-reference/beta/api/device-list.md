---
title: Listar dispositivos
description: 'Recupere uma lista de dispositivos registrados no diretório. '
author: spunukol
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 0766814c56315c63f60ade129443d8586016e90a
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50437104"
---
# <a name="list-devices"></a><span data-ttu-id="93556-103">Listar dispositivos</span><span class="sxs-lookup"><span data-stu-id="93556-103">List devices</span></span>

<span data-ttu-id="93556-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="93556-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="93556-105">Recupere uma lista de dispositivos registrados no diretório.</span><span class="sxs-lookup"><span data-stu-id="93556-105">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="93556-106">Permissões</span><span class="sxs-lookup"><span data-stu-id="93556-106">Permissions</span></span>

<span data-ttu-id="93556-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="93556-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


| <span data-ttu-id="93556-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="93556-109">Permission type</span></span> | <span data-ttu-id="93556-110">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="93556-110">Permissions (from least to most privileged)</span></span> |
|:--------------- |:------------------------------------------- |
| <span data-ttu-id="93556-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="93556-111">Delegated (work or school account)</span></span> | <span data-ttu-id="93556-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="93556-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span> |
| <span data-ttu-id="93556-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="93556-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="93556-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="93556-114">Not supported.</span></span> |
| <span data-ttu-id="93556-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="93556-115">Application</span></span> | <span data-ttu-id="93556-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93556-116">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="93556-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="93556-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /devices
```

## <a name="optional-query-parameters"></a><span data-ttu-id="93556-118">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="93556-118">Optional query parameters</span></span>

<span data-ttu-id="93556-119">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="93556-119">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="93556-120">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="93556-120">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="93556-121">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="93556-121">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="93556-122">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="93556-122">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="93556-123">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="93556-123">Request headers</span></span>

| <span data-ttu-id="93556-124">Nome</span><span class="sxs-lookup"><span data-stu-id="93556-124">Name</span></span> | <span data-ttu-id="93556-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="93556-125">Description</span></span> |
|:---- |:----------- |
| <span data-ttu-id="93556-126">Autorização</span><span class="sxs-lookup"><span data-stu-id="93556-126">Authorization</span></span>  | <span data-ttu-id="93556-p103">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="93556-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="93556-129">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="93556-129">ConsistencyLevel</span></span> | <span data-ttu-id="93556-130">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="93556-130">eventual.</span></span> <span data-ttu-id="93556-131">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, ou quando se usa `$filter` com o `$orderby` parâmetro de consulta.</span><span class="sxs-lookup"><span data-stu-id="93556-131">This header and `$count` are required when using `$search`, or when using `$filter` with the `$orderby` query parameter.</span></span> <span data-ttu-id="93556-132">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="93556-132">It uses an index that may not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="93556-133">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="93556-133">Request body</span></span>

<span data-ttu-id="93556-134">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="93556-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="93556-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="93556-135">Response</span></span>

<span data-ttu-id="93556-136">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [device](../resources/device.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93556-136">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="93556-137">Exemplos</span><span class="sxs-lookup"><span data-stu-id="93556-137">Examples</span></span>

### <a name="example-1-get-a-list-of-devices"></a><span data-ttu-id="93556-138">Exemplo 1: Obter uma lista de dispositivos</span><span class="sxs-lookup"><span data-stu-id="93556-138">Example 1: Get a list of devices</span></span>

#### <a name="request"></a><span data-ttu-id="93556-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93556-139">Request</span></span>

<span data-ttu-id="93556-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="93556-140">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="93556-141">HTTP</span><span class="sxs-lookup"><span data-stu-id="93556-141">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices
```
# <a name="c"></a>[<span data-ttu-id="93556-142">C#</span><span class="sxs-lookup"><span data-stu-id="93556-142">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="93556-143">JavaScript</span><span class="sxs-lookup"><span data-stu-id="93556-143">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="93556-144">Objective-C</span><span class="sxs-lookup"><span data-stu-id="93556-144">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="93556-145">Java</span><span class="sxs-lookup"><span data-stu-id="93556-145">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

#### <a name="response"></a><span data-ttu-id="93556-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="93556-146">Response</span></span>

<span data-ttu-id="93556-147">Veja a seguir um exemplo da resposta.</span><span class="sxs-lookup"><span data-stu-id="93556-147">Here is an example of the response.</span></span>
> <span data-ttu-id="93556-p105">Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93556-p105">Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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

### <a name="example-2-get-only-a-count-of-devices"></a><span data-ttu-id="93556-150">Exemplo 2: Obter apenas uma contagem de dispositivos</span><span class="sxs-lookup"><span data-stu-id="93556-150">Example 2: Get only a count of devices</span></span>

#### <a name="request"></a><span data-ttu-id="93556-151">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93556-151">Request</span></span>

<span data-ttu-id="93556-152">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93556-152">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/$count
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="93556-153">Resposta</span><span class="sxs-lookup"><span data-stu-id="93556-153">Response</span></span>

<span data-ttu-id="93556-154">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93556-154">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="93556-155">294</span><span class="sxs-lookup"><span data-stu-id="93556-155">294</span></span>

### <a name="example-3-use-filter-and-top-to-get-one-device-with-a-display-name-that-starts-with-a-including-a-count-of-returned-objects"></a><span data-ttu-id="93556-156">Exemplo 3: use $filter e $top para obter um dispositivo com um nome de exibição que comece com "a" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="93556-156">Example 3: Use $filter and $top to get one device with a display name that starts with 'a' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="93556-157">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93556-157">Request</span></span>

<span data-ttu-id="93556-158">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93556-158">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$filter=startswith(displayName, 'a')&$count=true&$top=1&$orderby=displayName 
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="93556-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="93556-159">Response</span></span>

<span data-ttu-id="93556-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93556-160">The following is an example of the response.</span></span>
><span data-ttu-id="93556-p106">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93556-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#devices",
  "@odata.count":1,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0",
      "hostNames":[]
    },
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000001",
      "deviceVersion":1,
      "displayName":"a_device_1",
      "Manufacturer":"Microsoft",
      "Model":"Surface",
      "operatingSystemVersion":"windows10EnterpriseN",
      "hostNames":["device_1.contoso.onmicrosoft.com", "device_1"]
    }
  ]
}
```

### <a name="example-4-use-search-to-get-devices-with-display-names-that-contain-the-letters-android-including-a-count-of-returned-objects"></a><span data-ttu-id="93556-163">Exemplo 4: use $search para obter dispositivos com nomes de exibição que contenham as letras "Android", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="93556-163">Example 4: Use $search to get devices with display names that contain the letters 'Android' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="93556-164">Solicitação</span><span class="sxs-lookup"><span data-stu-id="93556-164">Request</span></span>

<span data-ttu-id="93556-165">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="93556-165">The following is an example of the request.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices?$search="displayName:Android"&$count=true
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="93556-166">Resposta</span><span class="sxs-lookup"><span data-stu-id="93556-166">Response</span></span>

<span data-ttu-id="93556-167">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="93556-167">The following is an example of the response.</span></span>
><span data-ttu-id="93556-p107">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="93556-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#devices",
  "@odata.count":1396,
  "value":[
    {
      "accountEnabled":true,
      "deviceId":"00000000-0000-0000-0000-000000000000",
      "deviceVersion":1,
      "displayName":"contoso_Android",
      "Manufacturer":"Google",
      "Model":"Pixel 3a",
      "operatingSystemVersion":"10.0",
      "hostNames":[]
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
}
-->


