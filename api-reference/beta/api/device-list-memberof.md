---
title: Listar grupos de dispositivos
description: Obter grupos dos quais este dispositivo é membro direto. Essa operação não é transitiva.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: f6b869a51b0c81e2d80bd46da82fac69bf540fd1
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/10/2020
ms.locfileid: "48956411"
---
# <a name="list-device-groups"></a><span data-ttu-id="0de5b-104">Listar grupos de dispositivos</span><span class="sxs-lookup"><span data-stu-id="0de5b-104">List device groups</span></span>

<span data-ttu-id="0de5b-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0de5b-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0de5b-106">Obter grupos dos quais este dispositivo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="0de5b-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="0de5b-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="0de5b-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="0de5b-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="0de5b-108">Permissions</span></span>

<span data-ttu-id="0de5b-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="0de5b-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0de5b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="0de5b-111">Permission type</span></span>      | <span data-ttu-id="0de5b-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="0de5b-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0de5b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="0de5b-113">Delegated (work or school account)</span></span> | <span data-ttu-id="0de5b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0de5b-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0de5b-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="0de5b-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0de5b-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="0de5b-116">Not supported.</span></span>    |
|<span data-ttu-id="0de5b-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="0de5b-117">Application</span></span> | <span data-ttu-id="0de5b-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0de5b-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="0de5b-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="0de5b-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0de5b-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="0de5b-120">Optional query parameters</span></span>

<span data-ttu-id="0de5b-121">Este método dá suporte a [Parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search`, `$count`, e `$filter`.</span><span class="sxs-lookup"><span data-stu-id="0de5b-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="0de5b-122">A conversão OData também está habilitado, por exemplo, você pode convertê-la para obter apenas o directoryRoles do qual o usuário é membro.</span><span class="sxs-lookup"><span data-stu-id="0de5b-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="0de5b-123">Você pode usar `$search`na propriedade **displayName**.</span><span class="sxs-lookup"><span data-stu-id="0de5b-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="0de5b-124">Quando itens são adicionados ou atualizados para este recurso, eles são indexados especialmente para uso com os `$count` e `$search` parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="0de5b-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="0de5b-125">Pode haver um pequeno atraso entre quando um item é adicionado ou atualizado e quando está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="0de5b-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0de5b-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="0de5b-126">Request headers</span></span>
| <span data-ttu-id="0de5b-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="0de5b-127">Header</span></span>       | <span data-ttu-id="0de5b-128">Valor</span><span class="sxs-lookup"><span data-stu-id="0de5b-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0de5b-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="0de5b-129">Authorization</span></span>  | <span data-ttu-id="0de5b-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="0de5b-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0de5b-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="0de5b-132">ConsistencyLevel</span></span> | <span data-ttu-id="0de5b-133">eventualmente.</span><span class="sxs-lookup"><span data-stu-id="0de5b-133">eventual.</span></span> <span data-ttu-id="0de5b-134">Este cabeçalho e `$count` são necessários quando se utiliza `$search`, `$filter`, `$orderby` ou os parâmetros de consulta de conversão OData.</span><span class="sxs-lookup"><span data-stu-id="0de5b-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="0de5b-135">Ele usa um índice que pode não estar atualizado com as alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="0de5b-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0de5b-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="0de5b-136">Request body</span></span>
<span data-ttu-id="0de5b-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="0de5b-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0de5b-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de5b-138">Response</span></span>

<span data-ttu-id="0de5b-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="0de5b-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0de5b-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="0de5b-140">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-direct-member-of"></a><span data-ttu-id="0de5b-141">Exemplo 1: obter grupos dos quais o dispositivo é membro direto</span><span class="sxs-lookup"><span data-stu-id="0de5b-141">Example 1: Get groups that the device is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="0de5b-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0de5b-142">Request</span></span>

<span data-ttu-id="0de5b-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0de5b-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0de5b-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="0de5b-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="0de5b-145">C#</span><span class="sxs-lookup"><span data-stu-id="0de5b-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0de5b-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0de5b-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0de5b-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0de5b-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0de5b-148">Java</span><span class="sxs-lookup"><span data-stu-id="0de5b-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0de5b-149">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de5b-149">Response</span></span>

<span data-ttu-id="0de5b-150">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0de5b-150">The following is an example of the response.</span></span> 
> <span data-ttu-id="0de5b-151">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="0de5b-151">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="0de5b-152">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0de5b-152">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="0de5b-153">Exemplo 2: Obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="0de5b-153">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="0de5b-154">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0de5b-154">Request</span></span>

<span data-ttu-id="0de5b-155">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0de5b-155">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0de5b-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="0de5b-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="0de5b-157">C#</span><span class="sxs-lookup"><span data-stu-id="0de5b-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0de5b-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0de5b-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0de5b-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0de5b-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0de5b-160">Java</span><span class="sxs-lookup"><span data-stu-id="0de5b-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-count-only-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0de5b-161">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de5b-161">Response</span></span>

<span data-ttu-id="0de5b-162">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0de5b-162">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: text/plain
```

<span data-ttu-id="0de5b-163">394</span><span class="sxs-lookup"><span data-stu-id="0de5b-163">394</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="0de5b-164">Exemplo 3: usar a conversão OData e $search para obter associação com nomes de exibição que contenham as letras "vídeo" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="0de5b-164">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0de5b-165">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0de5b-165">Request</span></span>

<span data-ttu-id="0de5b-166">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0de5b-166">The following is an example of the request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="0de5b-167">HTTP</span><span class="sxs-lookup"><span data-stu-id="0de5b-167">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="0de5b-168">C#</span><span class="sxs-lookup"><span data-stu-id="0de5b-168">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0de5b-169">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0de5b-169">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0de5b-170">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0de5b-170">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0de5b-171">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de5b-171">Response</span></span>

<span data-ttu-id="0de5b-172">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0de5b-172">The following is an example of the response.</span></span>
><span data-ttu-id="0de5b-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0de5b-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.count":1396,
  "value":[
    {
      "displayName":"SFA Videos",
      "mail":"SFAVideos@service.contoso.com",
      "mailNickname":"SFAVideos"
    }
  ]
}
```

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="0de5b-175">Exemplo 4: usar a conversão OData e $filter para obter associação com um nome de exibição que comece com a letra "A", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="0de5b-175">Example 4: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="0de5b-176">Solicitação</span><span class="sxs-lookup"><span data-stu-id="0de5b-176">Request</span></span>

<span data-ttu-id="0de5b-177">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="0de5b-177">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="0de5b-178">HTTP</span><span class="sxs-lookup"><span data-stu-id="0de5b-178">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="0de5b-179">C#</span><span class="sxs-lookup"><span data-stu-id="0de5b-179">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-a-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0de5b-180">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0de5b-180">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-a-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0de5b-181">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0de5b-181">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-a-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0de5b-182">Java</span><span class="sxs-lookup"><span data-stu-id="0de5b-182">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-a-count-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0de5b-183">Resposta</span><span class="sxs-lookup"><span data-stu-id="0de5b-183">Response</span></span>

<span data-ttu-id="0de5b-184">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="0de5b-184">The following is an example of the response.</span></span>
><span data-ttu-id="0de5b-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="0de5b-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#directoryObjects",
  "@odata.count":76,
  "value":[
    {
      "displayName":"AAD Contoso Videos",
      "mail":"AADContosoVideos@contoso.com",
      "mailEnabled":true,
      "mailNickname":"AADContoso_Videos",
      "securityEnabled":true
    }
  ]
}
```
<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


