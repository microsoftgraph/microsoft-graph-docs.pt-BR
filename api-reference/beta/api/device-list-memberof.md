---
title: Listar grupos de dispositivos
description: Obter grupos dos quais este dispositivo é membro direto. Essa operação não é transitiva.
author: spunukol
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0788a4ceda260391acc89c3d290420635fe71c4e
ms.sourcegitcommit: 5a1373f2ccd9ee813fc60d42e7ac6b115b5f9f66
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/21/2020
ms.locfileid: "44333213"
---
# <a name="list-device-groups"></a><span data-ttu-id="65ff1-104">Listar grupos de dispositivos</span><span class="sxs-lookup"><span data-stu-id="65ff1-104">List device groups</span></span>

<span data-ttu-id="65ff1-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65ff1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="65ff1-106">Obter grupos dos quais este dispositivo é membro direto.</span><span class="sxs-lookup"><span data-stu-id="65ff1-106">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="65ff1-107">Essa operação não é transitiva.</span><span class="sxs-lookup"><span data-stu-id="65ff1-107">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="65ff1-108">Permissões</span><span class="sxs-lookup"><span data-stu-id="65ff1-108">Permissions</span></span>

<span data-ttu-id="65ff1-p103">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="65ff1-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65ff1-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="65ff1-111">Permission type</span></span>      | <span data-ttu-id="65ff1-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="65ff1-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="65ff1-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="65ff1-113">Delegated (work or school account)</span></span> | <span data-ttu-id="65ff1-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="65ff1-114">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="65ff1-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="65ff1-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="65ff1-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="65ff1-116">Not supported.</span></span>    |
|<span data-ttu-id="65ff1-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="65ff1-117">Application</span></span> | <span data-ttu-id="65ff1-118">Directory.Read.All, Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65ff1-118">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="65ff1-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="65ff1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="65ff1-120">Parâmetros de consulta opcionais</span><span class="sxs-lookup"><span data-stu-id="65ff1-120">Optional query parameters</span></span>

<span data-ttu-id="65ff1-121">Este método oferece suporte aos [parâmetros de consulta OData](/graph/query_parameters) para ajudar a personalizar a resposta, incluindo `$search` , `$count` e `$filter` .</span><span class="sxs-lookup"><span data-stu-id="65ff1-121">This method supports the [OData query parameters](/graph/query_parameters) to help customize the response, including `$search`, `$count`, and `$filter`.</span></span> <span data-ttu-id="65ff1-122">A conversão OData também é habilitada, por exemplo, você pode transmitir para obter apenas o directoryRoles do usuário é um membro.</span><span class="sxs-lookup"><span data-stu-id="65ff1-122">OData cast is also enabled, for example, you can cast to get just the directoryRoles the user is a member of.</span></span> <span data-ttu-id="65ff1-123">Você pode usar `$search` na propriedade **DisplayName** .</span><span class="sxs-lookup"><span data-stu-id="65ff1-123">You can use `$search` on the **displayName** property.</span></span> <span data-ttu-id="65ff1-124">Quando os itens são adicionados ou atualizados para esse recurso, eles são especialmente indexados para uso com os `$count` `$search` parâmetros de consulta e.</span><span class="sxs-lookup"><span data-stu-id="65ff1-124">When items are added or updated for this resource, they are specially indexed for use with the `$count` and `$search` query parameters.</span></span> <span data-ttu-id="65ff1-125">Pode haver um ligeiro atraso entre a adição ou atualização de um item e quando ele está disponível no índice.</span><span class="sxs-lookup"><span data-stu-id="65ff1-125">There can be a slight delay between when an item is added or updated and when it is available in the index.</span></span>

## <a name="request-headers"></a><span data-ttu-id="65ff1-126">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="65ff1-126">Request headers</span></span>
| <span data-ttu-id="65ff1-127">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="65ff1-127">Header</span></span>       | <span data-ttu-id="65ff1-128">Valor</span><span class="sxs-lookup"><span data-stu-id="65ff1-128">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="65ff1-129">Autorização</span><span class="sxs-lookup"><span data-stu-id="65ff1-129">Authorization</span></span>  | <span data-ttu-id="65ff1-p105">{token} de portador. Obrigatório.</span><span class="sxs-lookup"><span data-stu-id="65ff1-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="65ff1-132">ConsistencyLevel</span><span class="sxs-lookup"><span data-stu-id="65ff1-132">ConsistencyLevel</span></span> | <span data-ttu-id="65ff1-133">ocorra.</span><span class="sxs-lookup"><span data-stu-id="65ff1-133">eventual.</span></span> <span data-ttu-id="65ff1-134">Esse cabeçalho e `$count` são necessários ao usar os `$search` parâmetros de consulta de conversão de,, `$filter` `$orderby` ou OData.</span><span class="sxs-lookup"><span data-stu-id="65ff1-134">This header and `$count` are required when using the `$search`, `$filter`, `$orderby`, or OData cast query parameters.</span></span> <span data-ttu-id="65ff1-135">Ele usa um índice que pode não estar atualizado com alterações recentes no objeto.</span><span class="sxs-lookup"><span data-stu-id="65ff1-135">It uses an index that might not be up-to-date with recent changes to the object.</span></span> |

## <a name="request-body"></a><span data-ttu-id="65ff1-136">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="65ff1-136">Request body</span></span>
<span data-ttu-id="65ff1-137">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="65ff1-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="65ff1-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="65ff1-138">Response</span></span>

<span data-ttu-id="65ff1-139">Se bem-sucedido, este método retorna um código de resposta `200 OK` e uma coleção de objetos [directoryObject](../resources/directoryobject.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="65ff1-139">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="65ff1-140">Exemplos</span><span class="sxs-lookup"><span data-stu-id="65ff1-140">Examples</span></span>

### <a name="example-1-get-groups-that-the-device-is-a-direct-member-of"></a><span data-ttu-id="65ff1-141">Exemplo 1: obter grupos dos quais o dispositivo é membro direto</span><span class="sxs-lookup"><span data-stu-id="65ff1-141">Example 1: Get groups that the device is a direct member of</span></span>

#### <a name="request"></a><span data-ttu-id="65ff1-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65ff1-142">Request</span></span>

<span data-ttu-id="65ff1-143">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65ff1-143">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="65ff1-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="65ff1-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="c"></a>[<span data-ttu-id="65ff1-145">C#</span><span class="sxs-lookup"><span data-stu-id="65ff1-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65ff1-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65ff1-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65ff1-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65ff1-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65ff1-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="65ff1-148">Response</span></span>

<span data-ttu-id="65ff1-149">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65ff1-149">The following is an example of the response.</span></span> 
> <span data-ttu-id="65ff1-150">**Observação:** O objeto da resposta mostrado aqui pode estar truncado por motivos de concisão.</span><span class="sxs-lookup"><span data-stu-id="65ff1-150">**Note:** The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="65ff1-151">Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65ff1-151">All of the properties will be returned from an actual call.</span></span>
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

### <a name="example-2-get-only-a-count-of-all-memberships"></a><span data-ttu-id="65ff1-152">Exemplo 2: obter apenas uma contagem de todas as associações</span><span class="sxs-lookup"><span data-stu-id="65ff1-152">Example 2: Get only a count of all memberships</span></span>

#### <a name="request"></a><span data-ttu-id="65ff1-153">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65ff1-153">Request</span></span>

<span data-ttu-id="65ff1-154">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65ff1-154">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="65ff1-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="65ff1-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_count_only"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/$count
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="65ff1-156">C#</span><span class="sxs-lookup"><span data-stu-id="65ff1-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-count-only-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65ff1-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65ff1-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-count-only-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65ff1-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65ff1-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-count-only-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65ff1-159">Resposta</span><span class="sxs-lookup"><span data-stu-id="65ff1-159">Response</span></span>

<span data-ttu-id="65ff1-160">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65ff1-160">The following is an example of the response.</span></span>

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

<span data-ttu-id="65ff1-161">394</span><span class="sxs-lookup"><span data-stu-id="65ff1-161">394</span></span>

### <a name="example-3-use-odata-cast-and-search-to-get-membership-with-display-names-that-contain-the-letters-video-including-a-count-of-returned-objects"></a><span data-ttu-id="65ff1-162">Exemplo 3: usar a conversão OData e $search para obter associação com nomes de exibição que contenham as letras "vídeo" incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="65ff1-162">Example 3: Use OData cast and $search to get membership with display names that contain the letters 'Video' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="65ff1-163">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65ff1-163">Request</span></span>

<span data-ttu-id="65ff1-164">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65ff1-164">The following is an example of the request.</span></span> 


# <a name="http"></a>[<span data-ttu-id="65ff1-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="65ff1-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_video_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$search="displayName:Video"
ConsistencyLevel: eventual
```
# <a name="c"></a>[<span data-ttu-id="65ff1-166">C#</span><span class="sxs-lookup"><span data-stu-id="65ff1-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-video-count-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="65ff1-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="65ff1-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-video-count-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="65ff1-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="65ff1-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-video-count-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="65ff1-169">Resposta</span><span class="sxs-lookup"><span data-stu-id="65ff1-169">Response</span></span>

<span data-ttu-id="65ff1-170">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65ff1-170">The following is an example of the response.</span></span>
><span data-ttu-id="65ff1-p108">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65ff1-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

### <a name="example-4-use-odata-cast-and-filter-to-get-membership-with-a-display-name-that-starts-with-the-letter-a-including-a-count-of-returned-objects"></a><span data-ttu-id="65ff1-173">Exemplo 4: usar a conversão OData e $filter para obter associação com um nome de exibição que comece com a letra "A", incluindo uma contagem de objetos retornados</span><span class="sxs-lookup"><span data-stu-id="65ff1-173">Example 4: Use OData cast and $filter to get membership with a display name that starts with the letter 'A' including a count of returned objects</span></span>

#### <a name="request"></a><span data-ttu-id="65ff1-174">Solicitação</span><span class="sxs-lookup"><span data-stu-id="65ff1-174">Request</span></span>

<span data-ttu-id="65ff1-175">Este é um exemplo de solicitação.</span><span class="sxs-lookup"><span data-stu-id="65ff1-175">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "get_a_count"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/devices/{id}/memberOf/microsoft.graph.group?$count=true&$orderBy=displayName&$filter=startswith(displayName, 'A')
ConsistencyLevel: eventual
```

#### <a name="response"></a><span data-ttu-id="65ff1-176">Resposta</span><span class="sxs-lookup"><span data-stu-id="65ff1-176">Response</span></span>

<span data-ttu-id="65ff1-177">Este é um exemplo de resposta.</span><span class="sxs-lookup"><span data-stu-id="65ff1-177">The following is an example of the response.</span></span>
><span data-ttu-id="65ff1-p109">**Observação:** o objeto response mostrado aqui pode ser encurtado para legibilidade. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="65ff1-p109">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
